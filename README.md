Создал докер и по идее, чтобы всё работало, нужно написать в консоли команды docker build -t documentation-generator . и docker run -it --rm documentation-generator .
но ничего не работает, выдает ошибки:
как исправить не понимаю, как создать документацию с помощью докера тоже не понял.
PS C:\Users\vladm\IdeaProjects\javacoreGB> docker build -t documentation-generator .    
[+] Building 0.2s (1/1) FINISHED                                                                                                                                                                                     docker:default
=> [internal] load build definition from Dockerfile                                                                                                                                                                           0.1s
=> => transferring dockerfile: 2B                                                                                                                                                                                             0.0s
ERROR: failed to solve: failed to read dockerfile: open Dockerfile: no such file or directory

View build details: docker-desktop://dashboard/build/default/default/mnoqh2nbqxs9f51508p9autvv
PS C:\Users\vladm\IdeaProjects\javacoreGB> docker run -it --rm documentation-generator .
Unable to find image 'documentation-generator:latest' locally
docker: Error response from daemon: pull access denied for documentation-generator, repository does not exist or may require 'docker login': denied: requested access to the resource is denied.
See 'docker run --help'.
