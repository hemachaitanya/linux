FROM mcr.microsoft.com/dotnet/sdk:7.0
RUN apt update && apt install wget -y
RUN wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
RUN dpkg -i packages-microsoft-prod.deb
RUN mkdir -p /var/www/nopCommerce
WORKDIR /var/www/nopCommerce
RUN wget https://github.com/nopSolutions/nopCommerce/releases/download/release-4.60.4/nopCommerce_4.60.4_NoSource_linux_x64.zip
RUN apt-get install unzip && unzip nopCommerce_4.60.4_NoSource_linux_x64.zip
RUN mkdir bin logs 
EXPOSE 5000
CMD [ "dotnet", "Nop.Web.dll", "--urls", "http://0.0.0.0:5000"]
