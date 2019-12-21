node('master') {
		stage('Checkout from Git') {
		git credentialsId: 'git-credentials', url: 'https://github.com/prasadrayudu/hello-world.git'
		}
		stage('build Maven') {
		def mavenHome = tool name: 'Maven', type: 'maven'
		def mvncmd = "${mavenHome}\\bin\\mvn"
//	        bat "${mvncmd} clean package"
	        bat "${mvncmd} clean package"
		}
}
