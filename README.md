Main Specs:

The web app can be made using React, a Javascript framework used for making interactive UIs. A user accessing the app will be given the ability to make “conference rooms” and select the number of people and their email-IDs the user wants as participants to the conference.After confirming the number of participants and their emails, the recipients will be sent an invite link to the conference room on the app using the gmail api (https://developers.google.com/gmail/api/guides).

Once the app is open on the browser they will receive a prompt to provide a MetaMask wallet address they’d like to use. The app then prompts users to click a selfie they’d like to be used for confirming their identity. The capacitor api can be used to allow users to take selfies or select a pre-existing photo to upload as a selfie.
(https://capacitorjs.com/docs/apis/camera)

 When the users have uploaded their photos to Cere’s Decentralized Data Cloud they will receive a digital token and a content ID that represents their respective uploaded image to the DDC. Cere’s Freeport NFT contracts allow more than one digital content to be used as metadata for minting an NFT; thus, allowing more than one content ID to be attached to an NFT. This minted NFT can be used as an “Album” which represents all the participants of the conference. The app will then use freeport’s nft minter to mint the same number of NFTs as the original user entered as the number of participants and each participant will receive the ID for NFT in the wallet addresses provided. 


Testing Strategy:

For testing the webapp we can use Jest, a Javascript test runner that allows access to DOMs via jsdom. Jsdom is an approximation of the browser. For each test we can mount the React tree created onto a DOM element that is attached to the document, when the test ends we unmount the React tree from the document. For testing the rendering features, user triggered events there is a helper included in react-dom/test-utils called act() that ensures all updates related to the unit have been processed and applied to the DOM. For end-to-end testing, i.e. to make sure that the entire web app runs properly we can use a framework called Cypress.

Benefits for holding the NFT: 

If this app is being used in a work setting then the NFTs can be used as a way to reward bonuses to the owners. Hypothetically, if this app is used in the workplace to make a team for a project; on completion of the project the team leader can choose to reward NFT holders by staking the NFTs on the ethereum blockchain using cere’s cross-blockchain service. 
