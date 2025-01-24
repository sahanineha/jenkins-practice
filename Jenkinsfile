node {
    def path='/mnt/c/Users/sahan/OneDrive/Desktop/jenkins'
    stage('download-script') { 
        git 'https://github.com/sahanineha/jenkins-practice/blob/main/freespace.sh'
        echo "git-downloaded"
    }
    stage('run-script') {
        sh 'sh $path/freespace.sh'
        sh 'cat $path/freespace.txt'
    }
}
