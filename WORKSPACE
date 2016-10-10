workspace(name = "smyte")

# avro
new_http_archive(
    name = "avro_archive",
    url = "https://github.com/apache/avro/archive/release-1.8.1.tar.gz",
    strip_prefix = "avro-release-1.8.1",
    sha256 = "1bd406e161ca384c14a224cd12c9f6cb5f0b07924f7d52179f4e2691d1b91b50",
    build_file = "third_party/avro.BUILD",
)

bind(
    name = "avro",
    actual = "@avro_archive//:avro",
)

bind(
    name = "avrogen",
    actual = "@avro_archive//:avrogen",
)
# end of avro

# boost
new_http_archive(
    name = "boost_archive",
    url = "http://pilotfiber.dl.sourceforge.net/project/boost/boost/1.60.0/boost_1_60_0.tar.gz",
    sha256 = "21ef30e7940bc09a0b77a6e59a8eee95f01a766aa03cdfa02f8e167491716ee4",
    strip_prefix = "boost_1_60_0",
    build_file = "third_party/boost.BUILD",
)

bind(
    name = "boost",
    actual = "@boost_archive//:boost",
)
bind(
    name = "boost_context",
    actual = "@boost_archive//:context",
)
bind(
    name = "boost_filesystem",
    actual = "@boost_archive//:filesystem",
)
bind(
    name = "boost_iostreams",
    actual = "@boost_archive//:iostreams",
)
bind(
    name = "boost_program_options",
    actual = "@boost_archive//:program_options",
)
bind(
    name = "boost_regex",
    actual = "@boost_archive//:regex",
)
bind(
    name = "boost_system",
    actual = "@boost_archive//:system",
)
# end of boost

# double-conversion
new_http_archive(
    name = "double_conversion_archive",
    url = "https://github.com/google/double-conversion/archive/d4d68e4.tar.gz",
    strip_prefix = "double-conversion-d4d68e4e788bec89d55a6a3e33af674087837c82",
    sha256 = "4c21c78b4787051e682c7b5579ddb0c5fba823328faf14cdf52152a1f5bcdd32",
    build_file = "third_party/double-conversion.BUILD",
)

bind(
    name = "double_conversion",
    actual = "@double_conversion_archive//:double-conversion",
)
# end of double-conversion

# folly
new_http_archive(
    name = "folly_archive",
    url = "https://github.com/facebook/folly/archive/4cf30a1.tar.gz",
    strip_prefix = "folly-4cf30a1441af267ee42ab2fc9976dc3332f36ed8",
    build_file = "third_party/folly.BUILD",
)

bind(
    name = "folly",
    actual = "@folly_archive//:folly",
)

bind(
    name = "folly_config",
    actual = "//third_party/folly:config"
)
# end of folly

# gflags
http_archive(
    name = "gflags_archive",
    url = "https://github.com/gflags/gflags/archive/f4eace1.tar.gz",
    strip_prefix = "gflags-f4eace133187e0a101a6d6d71c55592b572de189",
    sha256 = "4bc2b2d677aaeb26a319fc58096976bf162ccdae66db8bb50a98a925d62f71fa",
)

bind(
    name = "gflags",
    actual = "@gflags_archive//:gflags",
)
# end of gflags

# glog
new_http_archive(
    name = "glog_archive",
    url = "https://github.com/google/glog/archive/0472b91.tar.gz",
    strip_prefix = "glog-0472b91c5defdf90cff7292e3bf7bd86770a9a0a",
    sha256 = "abb174454241c1c5b84f83d256a4bf0def8c1e725e3c06650f361e51def4005e",
    build_file = "third_party/glog.BUILD",
)

bind(
    name = "glog",
    actual = "@glog_archive//:glog",
)

bind(
    name = "glog_config",
    actual = "//third_party/glog:config"
)
# end of glog

# gtest
new_http_archive(
    name = "gtest_archive",
    url = "https://github.com/google/googletest/archive/release-1.8.0.tar.gz",
    strip_prefix = "googletest-release-1.8.0",
    sha256 = "58a6f4277ca2bc8565222b3bbd58a177609e9c488e8a72649359ba51450db7d8",
    build_file = "third_party/gtest.BUILD",
)

bind(
    name = "gtest",
    actual = "@gtest_archive//:gtest",
)

bind(
    name = "gtest_main",
    actual = "@gtest_archive//:gtest_main",
)

bind(
    name = "gmock",
    actual = "@gtest_archive//:gmock",
)

bind(
    name = "gmock_main",
    actual = "@gtest_archive//:gmock_main",
)
# end of gtest

# libevent
new_http_archive(
    name = "libevent_archive",
    url = "https://github.com/libevent/libevent/archive/release-2.0.22-stable.tar.gz",
    strip_prefix = "libevent-release-2.0.22-stable",
    sha256 = "ab89639b0819befb1d8b293d52047c6955f8d1c9150c2b22a0e6247930eb9128",
    build_file = "third_party/libevent.BUILD",
)

bind(
    name = "libevent",
    actual = "@libevent_archive//:libevent",
)

bind(
    name = "libevent_config",
    actual = "//third_party/libevent:config"
)
#end of libevent

# librdkafka
new_http_archive(
    name = "librdkafka_archive",
    url = "https://github.com/edenhill/librdkafka/archive/0.9.1.tar.gz",
    strip_prefix = "librdkafka-0.9.1",
    sha256 = "5ad57e0c9a4ec8121e19f13f05bacc41556489dfe8f46ff509af567fdee98d82",
    build_file = "third_party/librdkafka.BUILD",
)

bind(
    name = "librdkafka",
    actual = "@librdkafka_archive//:librdkafka",
)

bind(
    name = "librdkafka_config",
    actual = "//third_party/librdkafka:config"
)
# end of librdkafka

# libunwind
new_git_repository(
    name = "libunwind_git",
    remote = "git://git.sv.gnu.org/libunwind.git",
    tag = "v1.1", # Note: update the version in BUILD file
    build_file = "third_party/libunwind.BUILD",
)

bind(
    name = "libunwind",
    actual = "@libunwind_git//:libunwind",
)

bind(
    name = "libunwind_config",
    actual = "//third_party/libunwind:config"
)
# end of libunwind

# murmurhash3
new_http_archive(
    name = "murmurhash3_archive",
    url = "https://github.com/aappleby/smhasher/archive/61a0530.tar.gz",
    strip_prefix = "smhasher-61a0530f28277f2e850bfc39600ce61d02b518de",
    sha256 = "daa4bb23e24fe26a2f9d1bb0d241fff7eb963f7b7525fa20685e0dfb3b3ffa49",
    build_file = "third_party/murmurhash3.BUILD",
)

bind(
    name = "murmurhash3",
    actual = "@murmurhash3_archive//:murmurhash3",
)
# end of murmurhash3

# rocksdb
new_git_repository(
    name = "rocksdb_git",
    remote = "https://github.com/facebook/rocksdb.git",
    tag = "v4.8",
    build_file = "third_party/rocksdb.BUILD",
)

bind(
    name = "rocksdb",
    actual = "@rocksdb_git//:rocksdb",
)
# end of rocksdb

# snappy
new_http_archive(
    name = "snappy_archive",
    url = "https://github.com/google/snappy/archive/32d6d7d.tar.gz",
    strip_prefix = "snappy-32d6d7d8a2ef328a2ee1dd40f072e21f4983ebda",
    sha256 = "f50719c6dc7103d65df66882a3b4569d598eda251266463eca716928187dc12b",
    build_file = "third_party/snappy.BUILD",
)

bind(
    name = "snappy",
    actual = "@snappy_archive//:snappy",
)

bind(
    name = "snappy_config",
    actual = "//third_party/snappy:config"
)
# end of snappy

# wangle
new_http_archive(
    name = "wangle_archive",
    url = "https://github.com/facebook/wangle/archive/570f09e.tar.gz",
    strip_prefix = "wangle-570f09e3985746812875549d1c13204690505149",
    sha256 = "8306037414b6832774a05174a67d82ecc2595d90db7c321269288ef8bc86582d",
    build_file = "third_party/wangle.BUILD",
)

bind(
    name = "wangle",
    actual = "@wangle_archive//:wangle",
)
# end of wangle

# jemalloc
new_http_archive(
    name = "jemalloc_archive",
    url = "https://github.com/jemalloc/jemalloc/archive/4.2.1.tar.gz",
    strip_prefix = "jemalloc-4.2.1",
    sha256 = "38abd5c3798dee4bd0e63e082502358cd341b831b038bb443e89370df888a3eb",
    build_file = "third_party/jemalloc.BUILD",
)

bind(
    name = "jemalloc",
    actual = "@jemalloc_archive//:jemalloc",
)

bind(
    name = "jemalloc_config",
    actual = "//third_party/jemalloc:config"
)
# end of jemalloc

# zlib
new_http_archive(
    name = "zlib_archive",
    url = "https://github.com/madler/zlib/archive/v1.2.8.tar.gz",
    strip_prefix = "zlib-1.2.8",
    sha256 = "e380bd1bdb6447508beaa50efc653fe45f4edc1dafe11a251ae093e0ee97db9a",
    build_file = "third_party/zlib.BUILD",
)

bind(
    name = "zlib",
    actual = "@zlib_archive//:zlib",
)
# end of zlib
