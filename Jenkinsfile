pipeline{
 agent{
label {
 label 'QA'
 customWorkspace '/mnt/myproject'
 }
}
stages{ 
stage ('deploy'){
steps{
sh "sudo cp -r index.html 
/var/www/html/"
sh "sudo chmod -R 777 
/var/www/html/index.html"
}
}
stage ('start'){
steps{
sh "sudo yum install httpd -y"
 sh "service httpd start"
}
} 
}
 }

