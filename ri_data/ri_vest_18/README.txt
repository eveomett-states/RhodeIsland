2018 Rhode Island precinct and election shapefile.

## RDH Date retrieval
06/10/2021

## Sources
Election results from Rhode Island Board of Elections (https://www.ri.gov/election/results/2018/general_election/data/)
Precinct shapefile from the U.S. Census Bureau's 2020 Redistricting Data Program Phase 2 release.

## Fields metadata

Vote Column Label Format
------------------------
Columns reporting votes follow a standard label pattern. One example is:
G16PREDCli
The first character is G for a general election, P for a primary, S for a special, and R for a runoff.
Characters 2 and 3 are the year of the election.
Characters 4-6 represent the office type (see list below).
Character 7 represents the party of the candidate.
Characters 8-10 are the first three letters of the candidate's last name.

Office Codes
A## - Ballot amendment, where ## is an identifier
AGR - Commissioner of Agriculture
ATG - Attorney General
AUD - Auditor
CFO - Chief Financial Officer
CHA - Council Chairman
COC - Corporation Commissioner
COM - Comptroller
CON - State Controller
COU - City Council Member
CSC - Clerk of the Supreme Court
DEL - Delegate to the U.S. House
GOV - Governor
H## - U.S. House, where ## is the district number. AL: at large.
HOD - House of Delegates, accompanied by a HOD_DIST column indicating district number
HOR - U.S. House, accompanied by a HOR_DIST column indicating district number
INS - Insurance Commissioner
LAB - Labor Commissioner
LND - Commissioner of Public/State Lands
LTG - Lieutenant Governor
MAY - Mayor
MNI - State Mine Inspector
PSC - Public Service Commissioner
PUC - Public Utilities Commissioner
RGT - State University Regent
SAC - State Appeals Court (in AL: Civil Appeals)
SBE - State Board of Education
SCC - State Court of Criminal Appeals
SOC - Secretary of Commonwealth
SOS - Secretary of State
SPI - Superintendent of Public Instruction
SPL - Commissioner of School and Public Lands
SSC - State Supreme Court
TAX - Tax Commissioner
TRE - Treasurer
UBR - University Board of Regents/Trustees/Governors
USS - U.S. Senate

Party Codes
D and R will always represent Democrat and Republican, respectively.
See the state-specific notes for the remaining codes used in a particular file; note that third-party candidates may appear on the ballot under different party labels in different states.

## Fields
G18USSDWHI - Sheldon Whitehouse (Democratic Party)
G18USSRFLA - Robert G. Flanders Jr. (Republican Party)
G18USSOWRI - Write-in Votes

G18GOVDRAI - Gina M. Raimondo (Democratic Party)
G18GOVRFUN - Allan W. Fung (Republican Party)
G18GOVITRI - Joseph A. Trillo (Independent)
G18GOVIMUN - Luis-Daniel Muñoz (Independent)
G18GOVOGIL - William H. Gilbert (Moderate Party)
G18GOVOARM - Anne Armstrong (Compassion Party)
G18GOVOWRI - Write-in Votes

G18LTGDMCK - Daniel J. McKee (Democratic Party)
G18LTGRPEN - Paul E. Pence (Republican Party)
G18LTGIRIC - Jonathan J. Riccitelli (Independent)
G18LTGIMCC - Ross K. McCurdy (Independent)
G18LTGOHEL - Joel J. Hellmann (Moderate Party)
G18LTCOWRI - Write-in Votes

G18ATGDNER - Peter F. Neronha (Democratic Party)
G18ATGOGOR - Alan Gordon (Compassion Party)
G18ATGOWRI - Write-in Votes

G18TREDMAG - Seth Magaziner (Democratic Party)
G18TRERRIL - Michael G. Riley (Republican Party)
G18TREOWRI - Write-in Votes

G18SOSDGOR - Nellie M. Gorbea (Democratic Party)
G18SOSRCOR - Pat V. Cortellessa (Republican Party)
G18SOSOWRI - Write-in Votes

## Processing Steps

Several precincts in Providence were aligned with the city ward shapefile.

Limited ballots were reported by township. Federal ballots were reported by congressional district. These were distributed by candidate to precincts based on their share of the precinct-level vote for the given reporting unit.