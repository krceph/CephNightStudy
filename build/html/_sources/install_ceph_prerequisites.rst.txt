Prerequisites
=============

CEPH 설치를 위한 사전 작업을 진행합니다.

ceph-deploy setup
-----------------

.. code:: bash

    $ wget -q -O- 'https://download.ceph.com/keys/release.asc' | sudo apt-key add -
    $ echo deb https://download.ceph.com/debian-{ceph-stable-release}/ $(lsb_release -sc) main | sudo tee /etc/apt/sources.list.d/ceph.list
    $ sudo apt update
    $ sudo apt install ceph-deploy

