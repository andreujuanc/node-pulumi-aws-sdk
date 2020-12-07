FROM andreujuanc/lambada-base


#PULUMI 
#RUN curl -fsSL https://get.pulumi.com/ | sudo sh
RUN curl -fsSL https://get.pulumi.com | sudo sh -s -- --version 2.13.2
RUN mv ~/.pulumi /pulumi
ENV PATH "/pulumi/bin:${PATH}"

#AWS SDK
RUN curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
RUN unzip awscliv2.zip
RUN ./aws/install
