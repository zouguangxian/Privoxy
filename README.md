
# BUILDING

````bash
docker run --rm -it -v $PWD:/work dockcross/windows-static-x86 bash -c "sed -i s@/cdn-fastly.deb.debian.org/@/mirrors.aliyun.com/@g /etc/apt/sources.list && apt-get update && apt-get install -y nsis && cd windows && ./MYconfigure && make MAKENSIS=makensis -f GNUmakefile"
````
