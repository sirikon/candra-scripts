# CanDrA Scripts

Scripts for downloading, compiling and running
[CanDrA v+](https://bioinformatics.mdanderson.org/public-software/candra/).

## Requirements

`Bash`, `Perl`, `make`, `wget`, `tar`, `jq`.

## Usage

```bash
# Display help
./task

# Download CanDrA
./task download-candra

# List available databases
./task list-db
# Download database
./task download-db <key>

# Prepare installation
./task prepare
# Run CanDrA
./task run <db-key> <file>
```

### Example

```bash
./task run GENERAL ./installation/candra-plus/demo_input.txt
```

```tsv
Chrom	Coordinate	Ref_Allele	Mut_Allele	Strand	HGNC	mRNA	CONSEQUENCE	AAS	AAS_Location	CanDrA_Score	CanDrA_Category	CanDrA_Significance
10	89653809	G	T	+	PTEN	NM_000314	NON_SYNONYMOUS_CODING	G/V	36	10.9001	Driver	0.072175
2	209113112	G	T	-	IDH1	NM_005896	NON_SYNONYMOUS_CODING	R/L	132	7.4668	Driver	0.098198
2	209113113	G	T	+	IDH1	NM_005896	NON_SYNONYMOUS_CODING	R/S	132	7.4448	Driver	0.098421
3	178916876	C	T	-	PIK3CA	NM_006218	NON_SYNONYMOUS_CODING	R/Q	88	15.2451	Driver	0.048599
3	178936091	G	A	+	PIK3CA	NM_006218	NON_SYNONYMOUS_CODING	E/K	545	15.2092	Driver	0.051268
7	55259485	C	T	+	EGFR	NM_005228	NON_SYNONYMOUS_CODING	P/L	848	2.1587	Driver	0.19239
```
