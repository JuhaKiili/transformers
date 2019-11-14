FROM pytorch/pytorch:nightly-devel-cuda10.0-cudnn7
COPY download_glue_data.py /tmp
RUN python /tmp/download_glue_data.py --data_dir /glue_data
COPY requirements.txt /tmp
RUN pip install -r /tmp/requirements.txt
WORKDIR /workspace