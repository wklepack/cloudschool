# TYDZIEN 3

## Zadanie 1

> Zbuduj prosta konwencje nazewnicza dla min. takich zasobów jak Grupa Zasobów, VNET, Maszyn  Wirtualna, Dysk, Konta skladowania danych. Pamietaj o ograniczeniach w nazywaniu zasobów, które wystepuja w Azure.

Nie bede tutaj originalny bo zazwyczaj wspieram sie https://docs.microsoft.com/en-us/azure/architecture/best-practices/naming-conventions z malymi modyfikacjami.

# Stałe
```sh
Environment           : test, qa, uat (moze tego nie powinno byc :-) ), prod
Short_environment     : t,q,u,p
Location:             : us1, we1
```
# Konwencja

```sh
Resource Group    : <service_short_name>-<environment>-rg
Virtual Network   : <service_short_name>-<environment>-vnet
Virtual Machine   : <service_short_name>-<environment>-vm<fourn_number_digit>
Storage           : <service_short_name>-data<fourn_number_digit>
Disk              : <disktype>-disk<fourn_number_digit>
```

Jezeli nazwa jest za dluga to mozna uzywac kombiancji
# Skrócona konwencja
```sh
<service_name_3_letters_prefix><service_number><environment>,
czyli np. int740p  zapiast integrations-production
```
