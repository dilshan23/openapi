# openapi

#install java


#install openapi-gen

mkdir -p ~/bin/openapitools
curl https://raw.githubusercontent.com/OpenAPITools/openapi-generator/master/bin/utils/openapi-generator-cli.sh > ~/bin/openapitools/openapi-generator-cli
chmod u+x ~/bin/openapitools/openapi-generator-cli
export PATH=$PATH:~/bin/openapitools/




openapi-generator-cli generate -i swagger.yaml -g python-flask -o . -s

#specify library
openapi-generator-cli author template -g java --package-name webclient

