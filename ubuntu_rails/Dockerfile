# Copyright 2014 Alen Komic
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#    http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

FROM ubuntu

MAINTAINER akomic

ENV USER ak
ENV UID 1000

RUN apt-get update
RUN apt-get install -y ruby ruby-dev make libsqlite3-dev g++ zlib1g-dev patch libmysqlclient-dev
RUN gem install bundler rails
RUN useradd -d /home/${USER} -s /bin/bash -u ${UID} -m ${USER}
