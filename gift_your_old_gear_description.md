# Use Case Description: Process Gift Your Old Gear

## Use Case ID: UC3

### Level: User Goal

### Primary Actor: Customer

### Stakeholders and Interests:
- **Customer**: Wants to donate clothes and receive discount
- **Sales Assistant**: Needs to process donations efficiently and correctly
- **Charity Organizations**: Expect to receive usable clothing items
- **Store Manager**: Wants to maintain donation quality and track discounts
- **Viv's Vintage Wear**: Aims to promote sustainability and customer loyalty

### Preconditions:
1. System is operational
2. Sales Assistant is logged into the EPOS system
3. Customer has items to donate

### Success Guarantee (Postconditions):
1. Donation is recorded in the system
2. Customer receives 15% discount for their purchase
3. Donated items are marked for charity collection
4. Donation statistics are updated

### Main Success Scenario:
1. Customer brings items for donation to the Sales Assistant
2. Sales Assistant inspects each item for quality and usability
3. Sales Assistant confirms items meet donation criteria
4. System displays donation confirmation screen
5. Sales Assistant records the donation in the system:
   - Number of items
   - Type of items (clothing/accessories)
   - General condition
6. System generates donation receipt
7. System applies 15% discount to customer's next purchase
8. Sales Assistant places items in designated charity collection area
9. System updates donation statistics

### Extensions (Alternative Flows):
**1a. Customer inquires about donation criteria before bringing items**
1. Sales Assistant explains donation requirements
2. Customer decides whether to proceed with donation
3. Return to main flow

**2a. Items fail quality inspection**
1. Sales Assistant explains why items cannot be accepted
2. Customer retains items
3. Use case ends

**3a. Only some items meet criteria**
1. Sales Assistant separates acceptable from unacceptable items
2. Sales Assistant explains decisions to customer
3. Continue with main flow for acceptable items only
4. Customer retains rejected items

**7a. Customer has no immediate purchase**
1. System generates a discount voucher valid for 24 hours
2. Sales Assistant prints and hands voucher to customer
3. Use case ends

**7b. Customer attempts to use discount with other offers**
1. System blocks combination of discounts
2. Sales Assistant explains discount policy
3. Customer chooses which discount to apply
4. Continue with selected discount

### Special Requirements:
1. Quality inspection must be completed within 3 minutes per item
2. Donation processing should take no more than 5 minutes total
3. System must maintain accurate donation statistics
4. Donation receipts must be GDPR compliant

### Technology and Data Variations:
1. Donation recording can be done via:
   - EPOS system
   - Tablet device
   - Paper form (in case of system failure)
2. Discount can be applied via:
   - Direct system application
   - Printed voucher
   - Digital code

### Frequency of Occurrence:
- Approximately 20-30 donations per store per week
- Higher frequency during seasonal wardrobe changes (Spring/Fall)

### Miscellaneous:
1. Donation criteria must be clearly displayed at donation points
2. Staff training required for consistent quality assessment
3. Regular updates to charity partners about donation volumes
4. Monthly reporting of donation statistics required

### Business Rules:
1. 15% discount valid only on same-day purchase
2. Discount cannot be combined with other offers
3. No limit on number of items that can be donated
4. All donations must be in clean, wearable condition
5. Discount not applicable to gift card purchases

### Notes and Issues:
- Consider implementing digital receipt system for donations
- Potential for loyalty points integration
- Need for standardized quality assessment criteria
- Possibility of expanding to accessories and home items
