# set your parent image to be from the `ubuntu` repository and with the
# `18.04` tag
# --------------- #
FROM ubuntu:18.04
# --------------- #

# copy the contents of the current directory into the root directory (/)
# --------------- #
COPY . /
# --------------- #

# use `apt-get update` to update the index of packages in your docker container
# --------------- #
RUN apt-get update
# --------------- #

# use `apt-get` to install the `curl` and `ca-certificates` packages. you need
# to use the -y flag to automatically answer "yes" to all apt-get's questions
# --------------- #
RUN apt-get install curl ca-certificates  -y
# --------------- #

# define an environment variable `MYVAR` with default value `l33t`
# --------------- #
ENV MYVAR l33t
# --------------- #

# set the default launch command to invoke our shell script using `bash`
# that is, `bash gu511_download.sh`. remember that `docker` won't know what to
# do with that full command with a space in it...
# --------------- #
CMD ["bash","gu511_download.sh"]
# --------------- #
