node {

    stage('Pull Code from Git to Workspace') {
        git branch: 'main',
            url: 'https://github.com/Vandita30/space-science'
    }

    stage('Copy Workspace Files to NGINX html Folder') {
        bat '''
        @echo off
        echo Copying files from Jenkins workspace to NGINX html folder...

        xcopy "%WORKSPACE%\\*" "C:\\Users\\Administrator\\Downloads\\nginx-1.28.1\\html\\" /E /I /Y

        echo Files copied successfully.
        '''
    }
}

