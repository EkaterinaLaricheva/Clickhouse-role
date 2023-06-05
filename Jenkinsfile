node("linux"){
    stage("Git checkout"){
        git credentialsId: '5ac0095d-0185-431b-94da-09a0ad9b0e2c', url: 'https://github.com/EkaterinaLaricheva/Clickhouse-role
    }
    stage("Run playbook"){
            sh 'ansible-playbook site.yml -i inventory/prod.yml'
    }
}
