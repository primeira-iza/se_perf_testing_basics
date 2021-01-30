git clone https://github.com/primeira-iza/se_perf_testing_basics
cd se_perf_testing_basics
cd exercise_1
atom .
sudo docker run -d --name my-ghost -e url=http://localhost:3001 -p 3001:2368 ghost
sudo apt-get install python3-venv
python3 -m venv .venv
source .venv/bin/activate
pip install -U pip
pip install -U setuptools
pip install locust
locust -f locustfile.py
history
