FROM k8s.gcr.io/sig-storage/nfs-subdir-external-provisioner:v4.0.2
RUN git clone git@github.com:zisgood/imagesbuild.git
RUN mkdir -vp imagesbuild/sig-storage/nfs-subdir-external-provisioner
RUN tee imagesbuild/sig-storage/nfs-subdir-external-provisioner/Dockerfile  <<'EOF'
LABEL MAINTAINER=master@zisgood.top BUILDTYPE=Aliyun
EOF
RUN git add . && git commit -m "nfs-subdir-external-provisioner" && git push
