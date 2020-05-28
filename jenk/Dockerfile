FROM jenkins/jenkins:lts-centos

USER root

RUN dnf -y --disablerepo "github_git-lfs*" install 'dnf-command(config-manager)' && \
  dnf config-manager --disable "github_git-lfs*" && \
  dnf -y install ansible && \
  dnf clean all

