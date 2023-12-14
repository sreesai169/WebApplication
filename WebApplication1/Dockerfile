# Dockerfile

# Use the desired base image for your .NET app
FROM mcr.microsoft.com/dotnet/aspnet:8.0

# Set the working directory
WORKDIR /app

# Copy your .NET application files
COPY bin/Debug/net8.0/ .

# Copy the custom Nginx configuration file
COPY custom-nginx.conf /etc/nginx/conf.d/default.conf

# Expose the port on which your .NET app is listening
EXPOSE 5000

# Start your .NET app
ENTRYPOINT ["dotnet", "WebApplication1.dll"]
