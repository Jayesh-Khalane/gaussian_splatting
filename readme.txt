FFMPEG -i D:\gaussian-splatting\data\city\city.mp4 -qscale:v 1 -qmin 1 -vf fps=0.5 %04d.jpg

python convert.py -s D:\gaussian-splatting\data\city\

python train.py -s D:\gaussian-splatting\data\city\

SIBR_gaussianViewer_app -m  D:\gaussian-splatting\output\castle



conda activate gaussian_splatting