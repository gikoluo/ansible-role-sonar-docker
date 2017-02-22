# Ansible Role: SonarQube By Docker

Installs Sonar in docker container

## Requirements

gikoluo.docker
MySQL-Python

## Role Variables

Available variables are listed below, along with default values:

  mysql_image: "mysql:latest"
  mysql_container: "sonarqube-mysql"
  sonar_mysql_user: "sonar"
  sonar_mysql_password: "sonar"
  sonar_datanase_name: "sonar"

  sonar_image: "sonarqube:latest"
  sonar_port: 9000

## Dependencies

- gikoluo.docker - install docker first

## Example Playbook

    - hosts: all
      roles:
        - { role: gikoluo.sonar-docker }

## License

MIT

