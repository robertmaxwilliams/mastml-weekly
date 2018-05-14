1. Install docker on the host machine
2. `docker pull ubuntu`
3. `docker run -it ubuntu bash`
4. You should now be in the ubuntu shell
5. `apt-update`
6. `apt-install wget`
7. `wget https://repo.continuum.io/archive/Anaconda3-5.1.0-Linux-x86_64.sh`
8. `bash Anaconda3-5.1.0-Linux-x86_64.sh`
9. `export PATH=/root/anaconda3/bin:$PATH`
10. `conda create --name TEST_ML numpy scipy matplotlib pandas pymongo configobj nbformat scikit-learn
11. `source activate TEST_ML`
12. `conda install --channel matsci pymatgen`
13. `apt install git`
14. `git clone https://github.com/uw-cmg/MAST-ml`
15. `cd MAST-ml/examples/`
16. `sudo apt install libgl1-mesa-glx`
17. `pip install cython citrination_client`
18. `pip install --upgrade asn1crypto certifi cffi chardet citrination-client configobj cryptography cycler Cython decorator fastcache gmpy2 idna ipython-genutils jsonschema jupyter-core kiwisolver matplotlib mkl-fft mkl-random monty mpmath nbformat numpy palettable pandas pip pycparser PyDispatcher pymatgen pymongo pyOpenSSL pyparsing pypif PySocks python-dateutil pytz PyYAML requests ruamel.yaml scikit-learn scipy setuptools six spglib sympy tabulate tornado traitlets urllib3 wheel pip` (optional)
19. delete all print statements in setup.py (install vim)
20. python setup.py build
21. python setup.py install
22. `conda install --yes numpy scipy matplotlib`
23. `pip install citrination_client=="2.1.0"`
24. `git checkout ryan_updates_2018-03-08`
25. `apt install gcc`
26. we did it
27. python ../MASTML.py example_input.conf
