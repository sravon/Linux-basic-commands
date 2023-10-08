sudo groupadd devOpps
cat /etc/group | grep "devOpps"
sudo useradd devOpsEng -g "devOpps"
cat /etc/passwd | grep "devOpsEng"

mkdir os-concepts ubundu-is-the-best
cd os-concepts
touch file1.txt file2.txt
ls

cd ..
cd ubundu-is-the-best
touch file1.txt file2.txt
ls
ls -al
sudo chmod u=rw,g=r,o= file1.txt
sudo groupadd devOpsgroup
sudo chown devOpsEng:devOpsgroup file1.txt
ls -al
sudo usermod devOpsEng -g "devOpsgroup"
echo "hi,shrabon" > crash.in
cat crash.in
sed -i 's/shrabon/someone/g' crash.in
cat crash.in