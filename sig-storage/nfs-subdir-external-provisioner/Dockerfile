FROM k8s.gcr.io/sig-storage/nfs-subdir-external-provisioner:v4.0.2
RUN git clone git@github.com:zisgood/imagesbuild.git
mkdir -vp imagesbuild/sig-storage/nfs-subdir-external-provisioner
tee imagesbuild/sig-storage/nfs-subdir-external-provisioner/Dockerfile  <<'EOF'
LABEL MAINTAINER=master@zisgood.top BUILDTYPE=Aliyun
EOF
git add . && git commit -m "nfs-subdir-external-provisioner" && git push
