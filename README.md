## Possible solutions to some problems with Jupyter Notebook

Jupyter Notebook can be quite troublesome in use for several reasons, but IMO mainly because of the following fault

- Version control with git and GitHub: Changes in output (e.g.) causes git to make diffs in code, which is not wanted behaviour. 

It is difficult to collaborate when coding in Jupyter Notebook because of the problems with version control. Some possible solutions to this problems are presented in the following.  

### Docker

Dockerize. Make images that contain necessary software for running Jupyter Notebooks, with necessary packages (e.g. in 'requirements.txt'). *Does dockerization solve diff problems in git?!* At least this makes it very easy to ensure that the correct packages and correct software versions are installed, such that all collaborators have a working environment, across all operating systems.

There already exists some images on Docker Hub that could be used to begin with. 


### Pre-commit Hooks or Filters

Some links for how these solutions could be developed that might be of interest:

- [Pre-commit hooks](https://jamesfolberth.org/articles/2017/08/07/git-commit-hook-for-jupyter-notebooks/)
- [Git filters](https://pascalbugnion.net/blog/ipython-notebooks-and-git.html)
- [Description of several possibilites](http://timstaley.co.uk/posts/making-git-and-jupyter-notebooks-play-nice/)
- [Use nbconvert to 'clean'](https://tillahoffmann.github.io/2017/04/17/versioning-jupyter-notebooks-with-git.html)
- ['Clean' outputs while sharing cell outputs publicly](https://mg.readthedocs.io/git-jupyter.html)
- [Other options](https://nbsphinx.readthedocs.io/en/latest/usage.html#Using-Notebooks-with-Git)


### Developed Apps/Software

- Review Notebook App on GitHub marketplace could be of use to some. 
- [Nextjournal](https://nextjournal.com/), which seems to be based on Docker.
- [nbclean](https://github.com/choldgraf/nbclean): Clear cell outputs, filtering.etc. 
