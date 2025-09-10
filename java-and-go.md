# Commands for Java and Golang

Here are some common commands for Java and Golang, adapted from your provided file.

---

### **Java Commands**

#### Check Java Version and Installed JDK
* [cite_start]To check the Java version, use `java --version`[cite: 4].
* [cite_start]To check which JDK is installed, use `update-alternatives --config java`[cite: 5].

#### Install Downloaded JDK
* [cite_start]To install a downloaded `.deb` file for a JDK, use `dpkg -i jdk-24_linux-x64_bin.deb`[cite: 7].

#### Run a JAR file
* [cite_start]To run an executable `.jar` file, use `java -jar <filename>.jar`, for example `java -jar BurpLoaderKeygen.jar`[cite: 9].

---

### **Golang Commands**

#### Installation
* [cite_start]To install Golang, you can use the command: `rm -rf /usr/local/go && tar -C /usr/local -xzf go1.24.6.linux-amd64.tar.gz`[cite: 12].

#### Add Go Path and Apply Changes
* [cite_start]To add the Go path, you need to add the following lines to your shell profile, which can be opened with a command like `mousepad .zshrc` [cite: 14] [cite_start]or `mousepad .profile`[cite: 16]:
    * [cite_start]`export GOPATH=$HOME/go` [cite: 18]
    * [cite_start]`export GOROOT=/usr/local/go` [cite: 19]
    * [cite_start]`export PATH=$PATH:$GOROOT/bin:$GOPATH/bin` [cite: 20]
* [cite_start]After editing the file, apply the changes by running `source .zshrc` [cite: 15] [cite_start]or `source .profile`[cite: 16].
