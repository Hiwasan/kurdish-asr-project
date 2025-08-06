# Data Access and Management

## Important: Linguistic Data Security

The Kurdish linguistic corpus developed over 23 years of fieldwork is **not stored in this GitHub repository**. Due to the sensitive and proprietary nature of the linguistic data, all audio recordings, transcriptions, and translations are maintained in secure, access-controlled environments. Part of the dataset is stored at The Language Archive of Max Planck Institute for Psycholinguistics in Nijmegen (https://archive.mpi.nl/tla/)

## Dataset Overview

### Corpus Characteristics
- **Temporal Coverage**: 23 years of continuous linguistic fieldwork
- **Dialectal Diversity**: Multiple Kurdish dialect groups and regional variations
- **Data Quality**: Professional linguistic standards with verified transcriptions
- **Annotations**: Detailed linguistic metadata and cross-linguistic and parallel translations in English and Persian
- **Format**: High-quality audio recordings with time-aligned transcriptions

### Current Access Levels

#### Level 1: Sample Dataset (Current Phase)
- **Size**: 10-20 representative audio recordings
- **Purpose**: Initial ASR pipeline development and testing  
- **Access**: Secure cloud sharing with project collaborators
- **Duration**: Limited-time access for development purposes

#### Level 2: Development Dataset (Future Phase)
- **Size**: 100-200 recordings covering dialectal variations
- **Purpose**: Model training and optimization
- **Access**: After successful initial collaboration demonstration
- **Timeline**: Estimated 2-4 weeks from project initiation

#### Level 3: Full Corpus (Long-term)
- **Size**: Complete 23-year linguistic corpus
- **Purpose**: Comprehensive model development and evaluation
- **Access**: Requires formal collaboration agreement and demonstrated success
- **Timeline**: After establishing proven collaboration track record

## Data Security Protocols

### Access Management
- **Staged Access**: Incremental data access based on collaboration milestones
- **Secure Sharing**: Encrypted cloud storage with access controls and monitoring
- **Time Limitations**: All access grants have specified duration limits
- **Usage Restrictions**: Data limited to research collaboration purposes only

### Security Requirements
- **No Public Distribution**: Corpus data must never be made publicly available
- **No Unauthorized Sharing**: Data sharing limited to approved project collaborators
- **No Commercial Use**: Data restricted to research and academic purposes
- **Attribution Requirements**: All use must acknowledge data source and restrictions

## Data Format Specifications

### Audio Files
```
Format: WAV (uncompressed) / MP3 (high quality)
Sample Rate: 44.1kHz / 48kHz
Channels: Mono preferred for ASR processing
Duration: Variable (typically 30 seconds to 10 minutes per recording)
Quality: Professional field recording standards

```

### Transcription Format
```
Format: JSON/TXT with UTF-8 encoding
Structure: Time-aligned transcriptions when available
Languages: Kurdish (multiple dialects) with linguistic annotations
Metadata: Speaker demographics, dialect classification, recording context
```

### Translation Data
```
Format: Parallel text files (Kurdish → target languages)
Alignment: Sentence-level or phrase-level translation pairs
Quality: Professional linguistic translation standards
Coverage: Selected subset of corpus with verified translations
```

## Getting Started with Sample Data

### Step 1: Access Request
Contact the project lead for access to the current sample dataset. Access will be provided through secure cloud sharing with appropriate permissions.

### Step 2: Data Download and Setup
```bash
# Create local data directory (not tracked by Git)
mkdir -p data/sample_audio
mkdir -p data/sample_transcriptions
mkdir -p data/sample_translations

# Download sample data from secure sharing location
# (specific instructions provided with access credentials)
```

### Step 3: Data Verification
```bash
# Verify data integrity and format
python scripts/verify_sample_data.py

# Display dataset statistics
python scripts/data_stats.py --dataset sample
```

### Step 4: Initial Processing
```bash
# Convert to standard format for ASR processing
python src/preprocessing/format_audio.py --input data/sample_audio

# Prepare transcriptions for training
python src/preprocessing/prepare_transcriptions.py --input data/sample_transcriptions
```

## Data Usage Guidelines

### Permitted Uses
- **ASR Model Development**: Training and testing speech recognition models
- **Research Publication**: Academic research and publication (with proper attribution)
- **Technical Development**: Algorithm development and performance evaluation
- **Collaboration**: Shared development within approved project team

### Prohibited Uses
- **Public Distribution**: Making data available outside approved collaboration
- **Commercial Applications**: Using data for commercial product development
- **Unauthorized Research**: Research projects not covered by collaboration agreement
- **Data Mining**: Extracting data for purposes outside ASR development

## Data Update and Versioning

### Version Control
- **Sample Data**: Version controlled for consistency across development
- **Dataset Updates**: New data releases documented with version information
- **Format Changes**: Any format modifications communicated to all collaborators
- **Quality Improvements**: Ongoing transcription refinements and corrections

### Synchronization
- **Regular Updates**: Sample data refreshed based on collaboration progress
- **Format Consistency**: All collaborators working with identical data versions
- **Documentation**: Changes and updates documented in project communications

## Data Access Support

For questions about data access, format specifications, or technical issues:

1. **Technical Questions**: Contact technical lead for format and processing issues
2. **Access Requests**: Contact domain expert for permissions and security protocols  
3. **Usage Clarification**: Reach out for guidance on appropriate data usage
4. **Quality Issues**: Report any data quality concerns for resolution

## Future Data Integration

### Expansion Timeline
- **Month 1**: Sample dataset access and initial development
- **Month 2-3**: Development dataset access after milestone achievement
- **Month 4+**: Full corpus integration with formal agreements

### Access Criteria
- **Technical Milestone**: Successful ASR baseline implementation
- **Collaboration Success**: Demonstrated effective partnership
- **Security Compliance**: Adherence to data protection protocols
- **Research Progress**: Clear advancement toward project objectives

---

**Remember**: All linguistic data represents years of dedicated fieldwork and cultural engagement. Handle with appropriate respect, security, and professional standards.