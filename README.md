---


---

<p>Following are the tools required for the developement of backend services.</p>
<h1 id="intellij-community-edition"><strong>1) Intellij Community Edition</strong></h1>
<pre><code>sudo snap install intellij-idea-community --classic
</code></pre>
<h1 id="git"><strong>2) Git</strong></h1>
<pre><code>sudo apt install git
</code></pre>
<h1 id="jdk-jre-11"><strong>3) JDK JRE 11</strong></h1>
<pre><code>apt install openjdk-11-jre-headless
apt install openjdk-11-jdk-headless
</code></pre>
<h1 id="postman"><strong>4) Postman</strong></h1>
<pre><code>snap install postman
</code></pre>
<h1 id="elasticsearch"><strong><strong>5) Elasticsearch</strong></strong></h1>
<pre><code>sudo apt-get install apt-transport-https
wget -qO - https://artifacts.elastic.co/GPG-KEY-elasticsearch | sudo apt-key add -
add-apt-repository "deb https://artifacts.elastic.co/packages/7.x/apt stable main"
sudo apt-get update
sudo apt-get install elasticsearch
sudo /bin/systemctl enable elasticsearch.service
sudo systemctl start elasticsearch.service
</code></pre>
<h1 id="mysql"><strong><strong>6) MySQL</strong></strong></h1>
<pre><code>sudo apt update
sudo apt install mysql-server
sudo mysql_secure_installation    
sudo mysql
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'root';
FLUSH PRIVILEGES;
</code></pre>
<h1 id="setup-gradle"><strong><strong>7) Setup Gradle</strong></strong></h1>
<pre><code>wget https://services.gradle.org/distributions/gradle-6.5-bin.zip -P /tmp
unzip -d /opt/gradle /tmp/gradle-*.zip
vim /etc/profile.d/gradle.sh
</code></pre>
<blockquote>
<p>paste the following</p>
</blockquote>
<pre><code>export GRADLE_HOME=/opt/gradle/gradle-6.5
export PATH=${GRADLE_HOME}/bin:${PATH}
</code></pre>
<blockquote>
<p>press " <strong>:x</strong> " to save the file</p>
</blockquote>
<pre><code>chmod +x /etc/profile.d/gradle.sh
source /etc/profile.d/gradle.sh
</code></pre>
<h1 id="docker"><strong><strong>8) Docker</strong></strong></h1>
<pre><code>sudo apt update
sudo apt install apt-transport-https ca-certificates curl software-properties-common
curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo apt-key add -
sudo add-apt-repository "deb [arch=amd64] https://download.docker.com/linux/ubuntu bionic stable"
sudo apt update
apt-cache policy docker-ce
sudo apt install docker-ce
sudo docker images
sudo docker run hello world
</code></pre>
<h1 id="install-spring"><strong>9) Install Spring</strong></h1>
<pre><code>sudo apt install spring
</code></pre>
<h1 id="install-sticky-notes"><strong>10) Install Sticky notes</strong></h1>
<pre><code>sudo add-apt-repository ppa:umang/indicator-stickynotes  
sudo apt-get update  
sudo apt-get install indicator-stickynotes
</code></pre>

