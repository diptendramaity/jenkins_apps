node {

    stage('Pull Code from Git to Workspace') {
        git branch: 'main',
            url: 'https://github.com/diptendramaity/jenkins_apps'
    }

    stage('Copy Workspace Files to NGINX html Folder') {
        bat '''
        xcopy /E /I /Y "%WORKSPACE%/*" "C:/Users/Administrator/Downloads/nginx-1.28.1/html"
        '''
    }
}
