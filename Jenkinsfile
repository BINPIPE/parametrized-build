properties([parameters([choice(choices: 'master\nfeature-1\nfeature-2', description: 'Select Branch to build', name: 'branch')])])

node{
    stage('Scm Checkout'){
        echo "Pulling changes from the branch ${params.branch}"
        git url: 'https://github.com/BINPIPE/static-site-docker', branch: "${params.branch}"
    }
    
}
