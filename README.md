# About Sublist1r

Major shoutout to @aboul3la for building Sublist3r. (https://github.com/aboul3la/Sublist3r)[https://github.com/aboul3la/Sublist3r]
This repo is a single-threaded version of the same tool.

## Why?

Great question! I was building a passive recon tool on heroku. For those of you who have used heroku, know there is a 30 second request limit. To overcome this I spun up a celery dyno, to only then realize I could not use multithreading. I scoured the internet and realized a suprising amount of people were frustrated by celery limits, and a large amount were trying to use sublist3r. This is definitely a work in progress, but it works on heroku!

## Installation
```
git clone https://github.com/helenamerk/sublist1r.git
cd sublist1r
pip install -r requirements.txt
```

## Usage

## Usage

Short Form    | Long Form     | Description
------------- | ------------- |-------------
-d            | --domain      | Domain name to enumerate subdomains of
-b            | --bruteforce  | Enable the subbrute bruteforce module
-p            | --ports       | Scan the found subdomains against specific tcp ports
-v            | --verbose     | Enable the verbose mode and display results in realtime
-t            | --threads     | Number of threads to use for subbrute bruteforce
-e            | --engines     | Specify a comma-separated list of search engines
-o            | --output      | Save the results to text file
-h            | --help        | show the help message and exit

** Credit to Ahmed Aboul-Ela - @aboul3la for building the original Sublist3r.
