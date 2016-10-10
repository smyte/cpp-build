workspace(name = "smyte")

# avro
new_http_archive(
    name = "avro_git",
    url = "https://github.com/apache/avro/archive/release-1.8.1.zip",
    strip_prefix = "avro-release-1.8.1",
    sha256 = "6c2a5728bc0fd17a5c0a0ba1adfede0c8aa1e24cd035bc8643b3b3c533120a7a",
    build_file = "third_party/avro.BUILD",
)

bind(
    name = "avro",
    actual = "@avro_git//:avro",
)

bind(
    name = "avrogen",
    actual = "@avro_git//:avrogen",
)
# end of avro

# boost
new_http_archive(
    name = "boost_tgz",
    url = "http://pilotfiber.dl.sourceforge.net/project/boost/boost/1.60.0/boost_1_60_0.tar.gz",
    sha256 = "21ef30e7940bc09a0b77a6e59a8eee95f01a766aa03cdfa02f8e167491716ee4",
    strip_prefix = "boost_1_60_0",
    build_file = "third_party/boost.BUILD",
)

bind(
    name = "boost",
    actual = "@boost_tgz//:boost",
)
bind(
    name = "boost_context",
    actual = "@boost_tgz//:context",
)
bind(
    name = "boost_filesystem",
    actual = "@boost_tgz//:filesystem",
)
bind(
    name = "boost_iostreams",
    actual = "@boost_tgz//:iostreams",
)
bind(
    name = "boost_program_options",
    actual = "@boost_tgz//:program_options",
)
bind(
    name = "boost_regex",
    actual = "@boost_tgz//:regex",
)
bind(
    name = "boost_system",
    actual = "@boost_tgz//:system",
)
# end of boost

# double-conversion
new_http_archive(
    name = "double_conversion_git",
    url = "https://github.com/google/double-conversion/archive/d4d68e4.zip",
    strip_prefix = "double-conversion-d4d68e4e788bec89d55a6a3e33af674087837c82",
    sha256 = "7cf5fce1afc7698c6d56c71d93f2f655915d2282063ead40c4e0a2c97a957c56",
    build_file = "third_party/double-conversion.BUILD",
)

bind(
    name = "double_conversion",
    actual = "@double_conversion_git//:double-conversion",
)
# end of double-conversion

# folly
new_http_archive(
    name = "folly_git",
    url = "https://github.com/facebook/folly/archive/4cf30a1.zip",
    strip_prefix = "folly-4cf30a1441af267ee42ab2fc9976dc3332f36ed8",
    build_file = "third_party/folly.BUILD",
)

bind(
    name = "folly",
    actual = "@folly_git//:folly",
)

bind(
    name = "folly_config",
    actual = "//third_party/folly:config"
)
# end of folly

# gflags
http_archive(
    name = "gflags_git",
    url = "https://github.com/gflags/gflags/archive/f4eace1.zip",
    strip_prefix = "gflags-f4eace133187e0a101a6d6d71c55592b572de189",
    sha256 = "d90e767679e0c2ad01b51e7ffb21b2c63caeea9fad07fcc133d3b6f42c59bdb2",
)

bind(
    name = "gflags",
    actual = "@gflags_git//:gflags",
)
# end of gflags

# glog
new_http_archive(
    name = "glog_git",
    url = "https://github.com/google/glog/archive/0472b91.zip",
    strip_prefix = "glog-0472b91c5defdf90cff7292e3bf7bd86770a9a0a",
    sha256 = "710ee08a44e8384529ae0cd86cfca48940b485ab01e8b398dc32f8bb0913cf4f",
    build_file = "third_party/glog.BUILD",
)

bind(
    name = "glog",
    actual = "@glog_git//:glog",
)

bind(
    name = "glog_config",
    actual = "//third_party/glog:config"
)
# end of glog

# gtest
new_http_archive(
    name = "gtest_git",
    url = "https://github.com/google/googletest/archive/release-1.8.0.zip",
    strip_prefix = "googletest-release-1.8.0",
    sha256 = "f3ed3b58511efd272eb074a3a6d6fb79d7c2e6a0e374323d1e6bcbcc1ef141bf",
    build_file = "third_party/gtest.BUILD",
)

bind(
    name = "gtest",
    actual = "@gtest_git//:gtest",
)

bind(
    name = "gtest_main",
    actual = "@gtest_git//:gtest_main",
)

bind(
    name = "gmock",
    actual = "@gtest_git//:gmock",
)

bind(
    name = "gmock_main",
    actual = "@gtest_git//:gmock_main",
)
# end of gtest

# libevent
new_http_archive(
    name = "libevent_git",
    url = "https://github.com/libevent/libevent/archive/release-2.0.22-stable.zip",
    strip_prefix = "libevent-release-2.0.22-stable",
    sha256 = "84cd42f5ccba27868ec4e9176dfedb35fb87b34ef7d94c47c138ec3506a80677",
    build_file = "third_party/libevent.BUILD",
)

bind(
    name = "libevent",
    actual = "@libevent_git//:libevent",
)

bind(
    name = "libevent_config",
    actual = "//third_party/libevent:config"
)
#end of libevent

# librdkafka
new_http_archive(
    name = "librdkafka_git",
    url = "https://github.com/edenhill/librdkafka/archive/0.9.1.zip",
    strip_prefix = "librdkafka-0.9.1",
    sha256 = "62f64bd1b5fed505db0e9ba80bb5150dc981a75d813ab12f2b4da0b81a64f2f1",
    build_file = "third_party/librdkafka.BUILD",
)

bind(
    name = "librdkafka",
    actual = "@librdkafka_git//:librdkafka",
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
    name = "murmurhash3_git",
    url = "https://github.com/aappleby/smhasher/archive/61a0530.zip",
    strip_prefix = "smhasher-61a0530f28277f2e850bfc39600ce61d02b518de",
    sha256 = "950ab5345e43bf48ce2599f6c3f6ed711f20478f4a1b52763511bd4029d97656",
    build_file = "third_party/murmurhash3.BUILD",
)

bind(
    name = "murmurhash3",
    actual = "@murmurhash3_git//:murmurhash3",
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
    name = "snappy_git",
    url = "https://github.com/google/snappy/archive/32d6d7d.zip",
    strip_prefix = "snappy-32d6d7d8a2ef328a2ee1dd40f072e21f4983ebda",
    sha256 = "fe8099fc71349dd704f4af470ffffa1ad8d611195b7359075034f4e490c9e967",
    build_file = "third_party/snappy.BUILD",
)

bind(
    name = "snappy",
    actual = "@snappy_git//:snappy",
)

bind(
    name = "snappy_config",
    actual = "//third_party/snappy:config"
)
# end of snappy

# wangle
new_http_archive(
    name = "wangle_git",
    url = "https://github.com/facebook/wangle/archive/570f09e.zip",
    strip_prefix = "wangle-570f09e3985746812875549d1c13204690505149",
    sha256 = "3f95de1718937525f8d947623aab6a9a6ffb1d26e4cd07dfad615433df7e9fe7",
    build_file = "third_party/wangle.BUILD",
)

bind(
    name = "wangle",
    actual = "@wangle_git//:wangle",
)
# end of wangle

# jemalloc
new_http_archive(
    name = "jemalloc_git",
    url = "https://github.com/jemalloc/jemalloc/archive/4.2.1.zip",
    strip_prefix = "jemalloc-4.2.1",
    sha256 = "93f65652bbaffd42277815db7f13c685867d834e4dcbb7b8d1269b3c4012f618",
    build_file = "third_party/jemalloc.BUILD",
)

bind(
    name = "jemalloc",
    actual = "@jemalloc_git//:jemalloc",
)

bind(
    name = "jemalloc_config",
    actual = "//third_party/jemalloc:config"
)
# end of jemalloc

# zlib
new_http_archive(
    name = "zlib_git",
    url = "https://github.com/madler/zlib/archive/v1.2.8.zip",
    strip_prefix = "zlib-1.2.8",
    sha256 = "72290446e06e8962514d9226540b5277d3150a879afa0e6a88d98bc106f2fdc3",
    build_file = "third_party/zlib.BUILD",
)

bind(
    name = "zlib",
    actual = "@zlib_git//:zlib",
)
# end of zlib
