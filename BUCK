load('//:buckaroo_macros.bzl', 'buckaroo_deps')
load('//:subdir_glob.bzl', 'subdir_glob')

prebuilt_cxx_library(
  name = 'xpressive',
  header_only = True,
  header_namespace = 'boost',
  exported_headers = subdir_glob([
    ('include/boost', '**/*.hpp'),
    ('include/boost', '**/*.ipp'),
  ]),
  deps = buckaroo_deps(),
  visibility = [
    'PUBLIC',
  ],
)
