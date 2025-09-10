# Commands for Java and Golang

Here are some common commands for Java and Golang, adapted from your provided file.

---

### **Java Commands**

#### Check Java Version and Installed JDK
* To check the Java version, use `java --version`.
* To check which JDK is installed, use `update-alternatives --config java`.

#### Install Downloaded JDK
* To install a downloaded `.deb` file for a JDK, use `dpkg -i jdk-24_linux-x64_bin.deb`.

#### Run a JAR file
* To run an executable `.jar` file, use `java -jar <filename>.jar`, for example `java -jar BurpLoaderKeygen.jar`.

---

### **Golang Commands**

#### Installation
* To install Golang, you can use the command: `rm -rf /usr/local/go && tar -C /usr/local -xzf go1.24.6.linux-amd64.tar.gz`.

#### Add Go Path and Apply Changes
* To add the Go path, you need to add the following lines to your shell profile, which can be opened with a command like `mousepad .zshrc` or `mousepad .profile`:

  ```
  export GOPATH=$HOME/go

  export GOROOT=/usr/local/go
  
  export PATH=$PATH:$GOROOT/bin:$GOPATH/bin
  ```
* After editing the file, apply the changes by running `source .zshrc` [cite: 15] [cite_start]or `source .profile`.
