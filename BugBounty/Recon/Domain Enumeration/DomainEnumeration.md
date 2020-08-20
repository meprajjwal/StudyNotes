Subdomain Enumeration
	Tools and How to setup up with them & What commands and options works with which one and own review for each of them.

	Tools:
		Sublist3r
			sudo git clone https://github.com/aboul3la/Sublist3r
			cd Sublist3r
			sudo pip install -r requirements.txt

			Notes to install pip
				sudo apt-get install python-pip
				sudo apt-get install python3-pip

			Test whether the tool is working or not
				python Sublist3r.py -d <domain.com>

			//To do: list out more use cases for Sublist3r


			python /opt/tools/Sublist3r/sublist3r.py -d net-square.com

		Subbrute
			already integrated with the Sublist3r

			sudo git clone https://github.com/TheRook/subbrute.git

			to test single domain
				python subbrute.py google.com 
			To test multiple domains
				./subbrute.py google.com gmail.com blogger.com
			to test a newline delimited list of domains
				./subbrute.py -t list.txt

		Google Dorks

![GoogleDork Operator List](google-dork.jpg)
			eg.
				site:google.com
				site:google.com -www -cloud

		Knock

		Masscan

		Amass

	Notes: 
		Always check subdomains for both HTTP and HTTPS while checking which ones are valid.

