===============================================================================
# DDCLIENT v3.9.1

ddclient is a Perl client used to update dynamic DNS entries for accounts
on many dynamic DNS services.

===============================================================================

Dynamic DNS services currently supported include:

    vinaddns.com  - See http://vinaddns.com for details on obtaining a free account.
    DynDNS.com  - See http://www.dyndns.com for details on obtaining a free account.
    Hammernode  - See http://www.hn.org for details on obtaining a free account.
    Zoneedit    - See http://www.zoneedit.com for details.
    EasyDNS     - See http://www.easydns.com for details.
    NameCheap   - See http://www.namecheap.com for details
    ConCont     - See http://www.dydns.za.net for details
    DnsPark     - See http://www.dnspark.com for details
    DslReports  - See http://www.dslreports.com for details
    Sitelutions - See http://www.sitelutions.com for details
    Loopia      - See http://www.loopia.se for details
    Noip        - See http://www.noip.com/ for details
    Freedns     - See http://freedns.afraid.org/ for details
    ChangeIP    - See http://www.changeip.com/ for details
    dtdns       - See http://www.dtdns.com/ for details
    nsupdate    - See nsupdate(1) and ddns-confgen(8) for details
    CloudFlare  - See https://www.cloudflare.com/ for details
    Google      - See http://www.google.com/domains for details
    Duckdns     - See https://duckdns.org/ for details
    Freemyip    - See https://freemyip.com for details
    woima.fi    - See https://woima.fi/ for details
    Yandex      - See https://domain.yandex.com/ for details
    DNS Made Easy - See https://dnsmadeeasy.com/ for details
    DonDominio  - See https://www.dondominio.com for details
    NearlyFreeSpeech.net - See https://www.nearlyfreespeech.net/services/dns for details

DDclient now supports many of cable/dsl broadband routers.

Comments, suggestions and requests: use the issues on
	https://github.com/ddclient/ddclient/issues/new

The code was originally written by Paul Burry and is now hosted and maintained
through github.com. Please check out http://ddclient.net

-------------------------------------------------------------------------------
## INSTALLATION:

    sudo yum install ddclient

-------------------------------------------------------------------------------
## CONFIGURATION:

    vi /etc/ddclient.conf
        daemon=60
        syslog=yes
        #mail=root
        #mail-failure=root
        pid=/var/run/ddclient/ddclient.pid
        server=dns.vinaddns.com
        use=web
        protocol=dyndns2
        login=nnluc073
        password=X8AZO5DN8I
        phuta.vinaddns.com

-------------------------------------------------------------------------------
## TROUBLESHOOTING:

  1. enable debugging and verbose messages.
	 ``$ ddclient -daemon=0 -debug -verbose -noquiet``