# JMeter Installation Guide for macOS

## The Latest Version

Details of the latest version can be found on the
[JMeter Apache Project web site](https://jmeter.apache.org/)

## Step 1: Download JMeter

- Visit [JMeter Downloads](https://jmeter.apache.org/download_jmeter.cgi)
- Choose **Binaries** and download `apache-jmeter-5.6.3.tgz`
- Extract the file:
```bash
tar -xvzf apache-jmeter-5.6.3.tgz
```

## Step 2: Install Java JDK

- Download JDK for macOS from [Oracle JDK Downloads](https://www.oracle.com/java/technologies/downloads/#jdk24-mac)
- Follow the installation instructions.
- Verify Java installation:
```bash
java -version
```

## Step 3: Set JAVA_HOME

- Open `.zshrc` file:
```bash
nano ~/.zshrc
```
- Add the following:
```bash
export JAVA_HOME=$(/usr/libexec/java_home)
export PATH=$JAVA_HOME/bin:$PATH
```
- Save and apply changes:
```bash
source ~/.zshrc
```

## Step 4: Verify JMeter Setup

- Navigate to the `bin` directory:
```bash
cd /Users/Downloads/apache-jmeter-5.6.3/bin
```
- Check if `ApacheJMeter.jar` exists:
```bash
ls -la | grep ApacheJMeter.jar
```

## Step 5: Launch JMeter

- Run JMeter:
```bash
sh jmeter.sh
```
- The JMeter GUI should open.

## Additional Resources

- [JMeter Documentation](https://jmeter.apache.org/usermanual/index.html)

**JMeter is now successfully installed!**

**See screenshots below for reference.**

<img width="1341" alt="Screen Shot 2025-03-26 at 6 45 46 PM" src="https://github.com/user-attachments/assets/80b5ccb6-b54a-45b6-8387-3bfd21e92371" />


<img width="1344" alt="Screen Shot 2025-03-26 at 6 42 21 PM" src="https://github.com/user-attachments/assets/b775bdb1-a16d-4fc3-98e7-745341a93ba6" />


