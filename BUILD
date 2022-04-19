genrule(
    name = "hello",
    outs = ["hello.txt"],
    cmd = 'echo "Hello World" > $@',
)

genrule(
    name = "hello-slow",
    outs = ["hello-slow.txt"],
    cmd = 'sleep 5; echo "Hello World" > $@',
)

genrule(
    name = "hello-slow-dummy-srcs",
    srcs = ["src/dummy-src.txt"],
    outs = ["hello-slow-dummy-srcs.txt"],
    cmd = "sleep 5; echo $$(cat src/dummy-src.txt) > $@",
)
