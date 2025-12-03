# Containerlab
Repository per laboratori di rete con Containerlab 

### Tecnolige Utilizzate
* **Core:** Containerlab, Docker, Nokia SR Linux
* **Routing:** OSPF (Multi-Area), BGP (iBGP/eBGP), Static Routing
* **Tools:** Wireshark 

### Immagini utilizzate
 * **Nokia SR Linux:**  ghcr.io/nokia/srlinux
 * **Host:**  ghcr.io/hellt/network-multitool

## LAB 1 - Connettività base tra due host tramite un router
Configurazione del Default Gateway.

File Utili:
  * [Topologia Logica](./Lab_Subnet/topologia.png)
  * [File YAML](./Lab_Subnet/dualsubnet.clab.yml)
  * [File YAML con configurazione](./Lab_Subnet/dualsubnet_conf.clab.yml)
  * [Cartella con le configurazioni](./Lab_Subnet/configs)
  * [File pcap analisi traffico](./Lab_Subnet/cattura.pcap)

## LAB 2 - Routing Statico
Configurazione routing statico per stabilire e verificare la connetività end-to-end tra i nodi.

File utili:
  * [Topologia Logica](./Lab_RoutingStatico/topologia.png)
  * [File YAML](./Lab_RoutingStatico/routingStatico.clab.yml)
  * [File YAML con configurazione](./Lab_RoutingStatico/routingStatico_conf.clab.yml)
  * [Cartella con le configurazioni](.Lab_RoutingStatico/configs)

## LAB 3 - Routing Dinamico con OSPF
Implementazione di un'architettura IGP scalabile:
* Configurazione rouli router: ABR e ASBR.
* Ottimizzazione del LSDB tramite configurazione di **Stub Area**
* Redistribuzione controllata delle rotte.

File utili:
  * [Topologia Logica](./Lab_Routing_Dinamico/topologia.png)
  * [File YAML](./Lab_Routing_Dinamico/routingDinamico.clab.yml)
  * [Cartella con configurazioni parziali](./Lab_Routing_Dinamico/part_configs)
  * [File YAML con configurazione completa](./Lab_Routing_DInamico/routingDinamico_conf.clab.yml)
  * [Cartella con configurazioni complete](./Lab_Routing_Dinamico/configs)
  * [File pcap analisi traffico OSPF](./Lab_Routing_Dinamico/ospf.pcap)

## LAB 4 - Routing Inter-AS con BGP
Connessione tra 3 Autonomous Systems distinti:
* Implementazione di OSPF come IGP in uno dei tre AS. 
* Utilizzo di Route Reflectors.
* Manipolazione degli attributi di path BGP (Local Preference, MED, AS-Path Prepending) per direzionare il traffico.
* Applicazione di filtri sulle rotte e BFD per la convergenza rapida.

File utili:
  * [Topologia Logica](./Lab_Routing_InterAS/topologia.png)
  * [Schema delle sessioni BGP](./Lab_Routing_InterAS/SessioniBGP.png)
  * [File YAML](./Lab_Routing_InterAS/routingInterAS.clab.yml)
  * [Cartella con configurazioni iniziali](./Lab_Routing_InterAS/part_configs)
  * [File YAML con configurazione filtri](./Lab_Routing_InterAS/routingInterAS_filter.clab.yml)
  * [Cartella con configurazioni filtri](./Lab_Routing_InterAS/filter_configs)
  * [File pcap analisi traffico su Route Reflector](./Lab_Routing_InterAS/Route_Reflector.pcap)
  * [File YAML con configuraizone completa (modifca attributi BGP e BFD)](./Lab_Routing_InterAS/routingInterAS_conf.clab.yml)
  * [Cartella con configurazioni complete](./Lab_Routing_InterAS/configs)
  * [File pcap analisi traffico con attributi modificati](./Lab_Routing_InterAS/Path_Selection.pcap)
