# Linux-LA

1 Install Anaconda
  wget https://repo.anaconda.com/archive/Anaconda3-2022.05-Linux-x86_64.sh
  
2 Creat a conda env
  conda env create -f environment.yml
  
  'https://rabernat.github.io/research_computing/introduction-to-the-habanero-hpc-cluster.html'
  
3 Launch a notebook on a compute node
  qsub xxx.pbs

  (cat qsub xxx.pbs)

4 Connect to your notebook

  ssh -i /Users/tongya/Work/Cluster/LA/liutongya_rsa -L 9999:node67:8888 liutongya@124.160.91.130 -p 55555

  'https://rabernat.github.io/research_computing/running-jupyter-notebooks-on-habanero.html'

  or

  use xshell : 'https://github.com/JiachengHong/some-code/blob/main/run%20notebook%20on%20LA.pdf'

  grep Notebook test.e83786      see the token

  then open 'http://localhost:9999', input the token 

  enjoy it
