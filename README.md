# 2022-08-10-demo 


Simple demo for Anchore Enterprise, including Jenkins, CircleCI, Codefresh, and GitHub workflow examples.

Partial list of conditions that can be tested with this image:

1. xmrig cryptominer installed at `/xmrig/xmrig`
2. simulated AWS access key in `/aws_access`
3. simulated ssh private key in `/ssh_key`
4. selection of commonly-blocked packages installed (sudo, curl, etc)
5. `/log4j-core-2.14.1.jar` (CVE-2021-44228, et al)
6. CVE-2021-3156 (sudo) provided via hints file (rpm also available)
7. added anchorectl to demonstrate automatic go module detection (new in syft 0.42.0)
8. wide variety of ruby, node, python, java installed with different licenses
9. build drift detection via baseline dockerfile with minimal packages/dependencies
