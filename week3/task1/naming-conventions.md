#TYDZIEN3.1 �Zbuduj prosta konwencje nazewnicza dla min. takich zasob�w jak Grupa Zasob�w, VNET, Maszyn Wirtualna, Dysk, Konta skladowania danych. Pamietaj o ograniczeniach w nazywaniu zasob�w, kt�re wystepuja w Azure�

Nie bede tutaj originalny bo zazwyczaj wspieram sie https://docs.microsoft.com/en-us/azure/architecture/best-practices/naming-conventions z malymi modyfikacjami.


environment: test, qa, uat (fuuu), prod
short_environment: t,q,u,p
location: us1, we1

Resource Group 	: <service_short_name>-<environment>-rg
Virtual Network : <service_short_name>-<environment>-vnet
VM				: <service_short_name>-<environment>-<role>-vm<number>
Storage			: <service_short_name>-data<number>
OsDisk			: <disktype>-disk<number>

Jezeli nazwa jest za dluga to mozna uzywac kombiancji <service_name_3_letters_prefix><service_number><environment>, np. int740p (integrations-production)