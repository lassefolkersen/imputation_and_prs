
The first file - build.sh - is a copy of the standard NGC-HPC script to have docker images run on the NGC high-performance computer ("HPC"). Should work on computerome too, but haven't tested. The idea is basically to use the docker2singularity pluging to convert a dockerhub image to a .sif image, which can be run (almost) anywhere, even without being sudo. Then there's a lot of tinkering to make that .sif image work somewhere without admin-rights, because singularity rules are somewhat different than docker rules. But eventually it works, at least for vcf-input (sequencing)


