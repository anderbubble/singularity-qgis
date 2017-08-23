Bootstrap: docker
From: fedora:latest

%runscript

    echo "Starting QGIS (requires X11 forwarding)"
    exec $(which qgis)

%post

    echo "Installing QGIS"
    dnf update
    dnf -y install qgis qgis-python qgis-grass qgis-server
