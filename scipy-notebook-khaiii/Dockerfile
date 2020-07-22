FROM jupyter/scipy-notebook

USER root

# Install Khaiii
WORKDIR /deps
RUN git clone https://github.com/kakao/khaiii.git
WORKDIR /deps/khaiii

RUN pip install cython && \
  pip install --upgrade pip && \
  pip install -r requirements.txt && \
  mkdir build
WORKDIR /deps/khaiii/build

RUN cmake ..

RUN pwd
# RUN cmake .. && make all && make resource && make install && make package_python

# WORKDIR /deps/khaiii/build/package_python
# RUN pip install .

# # Add non-root user
# RUN adduser --disabled-password --gecos "" user

# # Reset Workdir
# WORKDIR /code