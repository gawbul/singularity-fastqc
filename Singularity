Bootstrap: docker
From: gawbul/docker-ubuntu1604-base

%postt
	mkdir -p /opt/tools
	cd /opt/tools
	wget -c http://www.bioinformatics.babraham.ac.uk/projects/fastqc/fastqc_v0.11.5.zip
	unzip fastqc_v0.11.5.zip
	cd FastQC
	chmod +x fastqc
	
%runscript
	exec /opt/tools/FastQC/fastqc "$@"
