# Copyright 2018 The Jetstack contributors.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

FROM debian:buster-slim

RUN apt-get -y update \
&& apt-get -y install --no-install-recommends \
   ca-certificates \
   curl \
   unzip \
&& curl https://releases.hashicorp.com/terraform/0.11.14/terraform_0.11.14_linux_amd64.zip -o terraform-0.11.zip \
&& unzip terraform-0.11.zip \
&& mv terraform /usr/local/bin/terraform-0.11 \
&& chmod +x /usr/local/bin/terraform-0.11 \
&& curl https://releases.hashicorp.com/terraform/0.12.4/terraform_0.12.4_linux_amd64.zip -o terraform-0.12.zip \
&& unzip terraform-0.12.zip \
&& mv terraform /usr/local/bin/terraform-0.12 \
&& chmod +x /usr/local/bin/terraform-0.12 \
&& rm -rf /var/lib/apt/lists/*
