# big-ip_asm_elk_integration

Repo in support to DC article
Contents:  
-sample_blocking_rdp_policy.xml <- this is a sample policy that can be used in conjunction with an as3 declaration to deploy a sec policy to BIG-IP.  
-sample_as3_declaration.json <- this is a sample AS3 declaration that will create an application complete with ASM policy and logging profile for ELK.  
  
The AS3 declaration is used to creat an application with:  
-Virtual Server (sample IP address 10.43.0.150).  
-Pool (two members 10.43.0.82:8000 and 10.43.0.82:8001).  
-An associated ASM Policy called My_ASM_Policy created from the XML file sample_blocking_rdp_policy.xml.  
-A logging profile defined in the AS3 declaration to send traffic to and ELK server (sample 10.45.0.79:5244).  

