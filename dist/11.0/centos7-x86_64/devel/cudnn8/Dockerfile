
FROM cuda:11.0-devel-centos7
LABEL maintainer "NVIDIA CORPORATION <sw-cuda-installer@nvidia.com>"

ENV CUDNN_VERSION 8.0.4.30
LABEL com.nvidia.cudnn.version="${CUDNN_VERSION}"

RUN yum install -y \
    libcudnn8-devel-${CUDNN_VERSION}-1.cuda11.0 \
    && yum clean all \
    && rm -rf /var/cache/yum/*
