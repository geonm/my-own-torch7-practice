w, dl_dw = model:getParameters() --w는 weights, dl_dw는 gradient parameter가 된다.

~ward(input, output)
model:backward(input,do_dw) -- 이를 수행했을 경우, dl_dw가 자동으로 업데이트 된다. 업데이트 전 dl_dw:zero() 필수

-------
-- torch debug IDE install
1. go to https://github.com/soumith/zbs-torch
2. follow the install guide
3. add torch7 env like this,
   1. sudo vim ~/.bashrc
   2.  export CUDA_HOME=/usr/local/cuda-8.0
       export LD_LIBRARY_PATH=${CUDA_HOME}/lib64
       export TORCH_BIN=/root/torch
   3. source ~/.bashrc

-- torch debug IDE RUN

0. open terminal
1. sudo su
2. cd zbs-torch
3. ./zbstudio.sh
