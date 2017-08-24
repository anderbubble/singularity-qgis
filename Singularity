Bootstrap: docker
From: fedora:latest

%runscript

    echo "Starting QGIS (requires X11 forwarding)"
    exec /usr/bin/qgis

%post

    echo "Installing QGIS"
    dnf -y install qgis qgis-python qgis-grass qgis-server

    echo "Cleaning up packages"
    dnf clean all

%test

    /usr/bin/qgis --help
