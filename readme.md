# Requisiti per utilizzare terraform con azure

* installare azure-cli
* installare terraform

# Setup

* fare login tramite azure-cli con il comando **az login**
* creare un file .tf per definire il provider azure come descritto nellla [documentazione] (https://registry.terraform.io/providers/hashicorp/azurerm/latest/docs)
* lanciare il comando **terraform init** per inizializzare terraform

# Utilizzo base

una volta definite le risorse da instanziare negli appositi file .tf utilizzare i seguenti comandi:

* terraform plan: analizza lo stato corrente dell'infrastruttura e produce il piano di deploy per allineare lo stato attuale con lo stato definito nei file di configurazione
* terraform apply: esegue gli step definiti con il comando plan
* terraform destroy: cancella tutte le risorse dell'infrastruttura
* (terraform refresh): per fare un update dello stato attuale dell'infrastruttura
