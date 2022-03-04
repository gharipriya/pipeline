pipeline {
	agent { label 'node1'}
	stages {
				stage('Build') { 
					steps {
						<project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
						xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
						<modelVersion>4.0.0</modelVersion>
						<groupId>com.efsavage</groupId>
						<artifactId>hello-world-war</artifactId>
						<version>1.0.0</version>
						<packaging>war</packaging>
						<name>Hello World Web Application Repository</name>
						<description>Simplest possible Java Webapp</description>

	<build>
		<plugins>
			<plugin>
				<groupId>org.mortbay.jetty</groupId>
				<artifactId>jetty-maven-plugin</artifactId>
				<version>8.1.5.v20120716</version>
				<configuration>
					<scanIntervalSeconds>0</scanIntervalSeconds>
				</configuration>
			</plugin>
			<plugin>
				<groupId>org.apache.maven.plugins</groupId>
				<artifactId>maven-war-plugin</artifactId>
				<version>2.1.1</version>
			</plugin>
		</plugins>
	</build>

</project>
						
					}
				}	
				stage('Test'){
					steps {
						sh '''
							sleep 15
							echo "This is a Test stage"
						'''	
					}
				}
		stage('Deploy'){
			steps {
				sh '''
					sleep 5
					echo "This is a Deploy stage"
				'''
			}
		}
		
		stage('My-stage'){
			steps {
				sh '''
					sleep 5
					echo "This is a My-stage stage"
				'''
			}
		}	
	}
}
