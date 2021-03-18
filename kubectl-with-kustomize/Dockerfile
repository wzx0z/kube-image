FROM alpine:3.8

ENV KUSTOMIZE_VERSION v3.8.5
ENV KUBECTL_VERSION 1.19.3

RUN wget -c https://github.com/kubernetes-sigs/kustomize/releases/download/kustomize/${KUSTOMIZE_VERSION}/kustomize_${KUSTOMIZE_VERSION}_linux_amd64.tar.gz -O - | tar -xz && \
  chmod +x kustomize && \
  mv kustomize /usr/local/bin/kustomize

RUN wget -O /usr/local/bin/kubectl https://storage.googleapis.com/kubernetes-release/release/v${KUBECTL_VERSION}/bin/linux/amd64/kubectl && \
  chmod +x /usr/local/bin/kubectl
