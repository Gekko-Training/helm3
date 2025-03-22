docker run --rm -it -d \
  -p 8282:8080 \
  -e DEBUG=1 \
  -e STORAGE=local \
  -e STORAGE_LOCAL_ROOTDIR=/charts \
  -v /tmp/ChartMuseumRepo:/charts \
  --name chartmuseum \
  ghcr.io/helm/chartmuseum:v0.14.0