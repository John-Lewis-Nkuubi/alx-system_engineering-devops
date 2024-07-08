## 0-custom_http_response_header
### Requirements:
- Configure Nginx so that its HTTP response contains a custom header (on web-01 and web-02)
- The name of the custom HTTP header must be X-Served-By
- The value of the custom HTTP header must be the hostname of the server Nginx is running on
- Write 0-custom_http_response_header so that it configures a brand new Ubuntu machine to the requirements asked in this task
- Ignore SC2154 for shellcheck

## 1-install_load_balancer
### Requirements:
- Configure HAproxy so that it send traffic to web-01 and web-02
- Distribute requests using a roundrobin algorithm
- Make sure that HAproxy can be managed via an init script
- Make sure that your servers are configured with the right hostnames: [STUDENT_ID]-web-01 and [STUDENT_ID]-web-02.
For your answer file, write a Bash script that configures a new Ubuntu machine to respect above requirements

## 2-puppet_custom_http_response_header.pp
### Requirement
- Automate the task of creating a custom HTTP header response, but with Puppet.
- The name of the custom HTTP header must be X-Served-By
- The value of the custom HTTP header must be the hostname of the server Nginx is running on
- Write 2-puppet_custom_http_response_header.pp so that it configures a brand new Ubuntu machine to the requirements asked in this task
