node{
    stage('Clone') {
        checkout scm
    }
    stage('Ansible') {
      ansiblePlaybook (
          colorized: true, 
          become: true,             
          playbook: 'playbook.yml',
          inventory: 'hosts.yml'
      )
    }
    stage('Ansible2') {
      ansiblePlaybook (
          colorized: true, 
          become: true,             
          playbook: 'playbook2.yml',
          inventory: 'hosts.yml'
      )
    }
    stage('Ansible3') {
      ansiblePlaybook (
          colorized: true, 
          become: true,             
          playbook: 'playbook3.yml',
          inventory: 'Clienthost.yml'
      )
    }    
}