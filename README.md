# Motion Blur Before an Upscale: The Cutoff Is Already Written, and Sharpening Cannot Move It

A 1-D motion blur of length L removes everything above 0.911/L cycles per pixel. Measured transfer matches the closed form within 1.0%, 2x/4x upscaling moves that cutoff by under 0.5%, and Wiener deconvolution gains 6.5 dB on detailed crops and loses 9.8 dB on flat ones. Optimal sharpen radius is 0.39*L; a horizontal-only mask only wins within 32 degrees of horizontal.

**Read it with the tables and the reproduction snippets:** <https://celticgemini001.github.io/upgolab-motion-blur-before-upscale/>

## About this repo

This repository exists to serve one measured article. Every number in it came from
ffmpeg and numpy run on real files on this machine — the commands are in the page so
you can re-run them and get the same rows. Where the measurement contradicted the
hypothesis, the page says so.

## The tool behind the notes

<https://upgolab.com> — browser-based AI upscaler for photos and short video.

## Index

All the guides are cross-linked from the hub:
<https://celticgemini001.github.io/upgolab-tools/>
