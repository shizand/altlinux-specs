# altlinux-specs

```
docker run --rm -it --privileged -v $(pwd):/usr/src/project ghcr.io/shizand/altlinux-builder
cd /usr/src/project/...
rpmgs *.spec
rpmbs -b p10 *.spec
hsh /home/user/RPM/SRPMS/* --no-sisyphus-check=packager,gpg,changelog
cp ~/hasher/repo/x86_64/RPMS.hasher/* .
```