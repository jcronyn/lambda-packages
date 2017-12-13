##Build

On an machine with Amazon Linux:

`./build.sh cryptography 1.9`

On a machine with docker and access to lambci images:

`docker run --rm -v `pwd`:/app -d lambci/lambda:build-python2.7 bash -c "cd /app && /app/build.sh --docker --py2-only cryptography 1.9"`

`docker run --rm -v `pwd`:/app -d lambci/lambda:build-python3.6 bash -c "cd /app && /app/build.sh --docker --py3-only cryptography 1.9"`
