FROM mcr.microsoft.com/windows/nanoserver:sac2016

ADD ./bin/* /redis/
RUN setx PATH '%PATH%;C:\Redis\'

WORKDIR /Redis/

EXPOSE 6379

# Define our command to be run when launching the container
CMD .\redis-server.exe .\redis.windows.conf --port 6379