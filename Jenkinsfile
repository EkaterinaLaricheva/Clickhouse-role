node("linux"){
    stage("Git checkout"){
        git credentialsId: url: 'https://github.com/EkaterinaLaricheva/Clickhouse-role.git'
    }
    stage("Sample define secret_check"){
        secret_check=true
    }
    stage("Run playbook"){
        if (secret_check){
            sh 'ansible-playbook site.yml -i inventory/prod.yml'
        }
        else{
            echo 'need more action'
        }
        
    }
}
