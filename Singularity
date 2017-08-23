Bootstrap: docker
From: fedora:latest

%runscript

    echo "Starting QGIS (requires X11 forwarding)"
    exec $(which qgis)

%post

    echo "Updating Fedora"
    dnf -y update

    echo "Installing QGIS"
    dnf -y install qgis qgis-python qgis-grass qgis-server

    echo "Cleaning up packages"
    dnf clean all
