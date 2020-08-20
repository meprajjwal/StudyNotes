
BruteForce
	The traditional way
		Bruteforce :
			sublist3r
			enumaill
			massdns
			altdns
			brutesubs
			dns-parallel-prober
			dnscan
			knockpy
			tko-subs
			HostileSubBruteForce
		Find a pattern (.dev, .corp, .stage)
		Brute force again
			Different permutations
			Different environment

		Google Dork: site.com -www -cdn


Amazon Web Services
	Look for S3 buckets (site:s3.amazonaws.com +...)
	AWS instances (site:amazonaws.com -s3)
	Use Google for patterns
	Github
	Automate your work

Automation
	Create a list of subdomains
	Create a list of environments
		Prod
		Stage
		Dev
	Automate
	Catch them all
	Tools:
		Amazon S3 Bucket finder
		SandCastle by YasinS
		BucketFinder by digi-ninja

	AWS Recon - what could go wrong?
		S3 bucket not owned by company
		You may be out of scope
		The S3 bucket doesn't contain any sensite info
		Third party apps

Github
	Github Recon
		Environments (dev, stage, prod)
		Secret Keys (API_Keys, AWS_Secret, etc)
		Internal credentials
		API endpoints
		Domain patterns

		"levelup.com" "dev"
		"dev.levelup.com"
		"levelup.com" API_key
		"levelup.com" password
		"api.levelup.com"

		Google Dork: site:"Github.com" + "ORG" + ...

	Tools:
		gitrob
		git-all-secrets
		truffleHog
		git-secrets
		repo-supervisor

	What could go wrong?
		Employee no longer works at the company.
		Old secret_keys
		The S3 bucket doesn't contain any sensitive info
		Third party apps

Asset Identification
	Get Creative
		Censys.io
		Shodan.io
		Archive.org
		.JS File
			Endpoints
			Credentials
			More (internal) subdomains


=========================================
What Things to consider while reconing?
========

    Enumerate domains
    Enumerate subdomains
    Resolve subdomains
    Test for CORS
    Test for subdomain takeover
    Scan for open ports
    Make a list of Web apps
    Do network tests on non HTTP ports
    Take screenshots for visual identification
    Run Web app scanners on the list of Web apps
    Run CMS scanners
    Do files & directory bruteforce
    Enumerate JS files
    Get secrets & new endpoints from JS files
    Look for known vulnerabilities based on identified service & library versions
    Do parameter bruteforcing
    Github recon
    Test for AWS misconfigurations
    Google dorking




