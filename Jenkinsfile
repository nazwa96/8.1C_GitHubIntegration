{\rtf1\ansi\ansicpg1252\cocoartf2821
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\fs24 \cf0 pipeline \{\
    agent any\
    stages \{\
        stage('Build') \{\
            steps \{ echo 'Build with Maven or Gradle' \}\
        \}\
        stage('Unit & Integration Tests') \{\
            steps \{ echo 'Run JUnit + Selenium tests' \}\
        \}\
        stage('Code Analysis') \{\
            steps \{ echo 'Static code analysis via SonarQube' \}\
        \}\
        stage('Security Scan') \{\
            steps \{ echo 'Dependency check with OWASP DC' \}\
        \}\
        stage('Deploy to Staging') \{\
            steps \{ echo 'Deploy Docker image to AWS EC2' \}\
        \}\
        stage('Integration Tests on Staging') \{\
            steps \{ echo 'API tests with Postman Newman' \}\
        \}\
        stage('Deploy to Production') \{\
            steps \{ echo 'kubectl apply -f k8s/' \}\
        \}\
    \}\
\}\
}