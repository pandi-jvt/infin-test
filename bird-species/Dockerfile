FROM tensorflow/tensorflow
 
RUN pip install tensorflow
RUN pip install boto3
RUN pip install mlflow
RUN pip install tensorflow_datasets
RUN pip install pandas
RUN pip install numpy

ARG IGNORECACHE=12
RUN echo "$IGNORECACHE"
RUN python3 -m pip install --no-cache-dir http://vmi504080.contaboserver.net:9876/packages/concurrent-plugin/concurrent_plugin-0.4.9-py3-none-any.whl
RUN python3 -m pip install --no-cache-dir http://cvat.infinstor.com:9876/packages/infinstor/infinstor-2.0.63-py3-none-any.whl
# RUN python3 -m pip install --upgrade http://cvat.infinstor.com:9876/packages/infinstor/infinstor-2.0.63-py3-none-any.whl