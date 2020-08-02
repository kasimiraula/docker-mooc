FROM ubuntu:16.04 

WORKDIR /mydir
RUN apt-get update && apt-get install -y curl
COPY curl_script.sh .
RUN chmod u+x curl_script.sh
CMD ["/bin/bash", "curl_script.sh"]

