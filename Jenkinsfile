node('master') {
		stage('Checkout from Git') {
		git credentialsId: 'git-credentials', url: 'https://github.com/prasadrayudu/hello-world.git'
		}
		stage('build Maven') {
		def MavenHome = tool name: 'Maven', type: 'maven'
			def mvnCmd = "${mavenHome}\bin\mvn"
			sh "${mvnCmd} clean package"
		}
}
