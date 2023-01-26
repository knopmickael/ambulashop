Category {
	name: string,
	_factory: Category[
		{name: 'feira/frutas'},
		{name: 'acai/sorvetes'},
		{name: 'guloseimas/balas/chicletes'},
		{name: 'roupas/vestimenta'},
		{name: 'geral/eletronicos'},
		{name: 'criancas/brinquedos'}
	]
}

Address {
	details: string
}

Contact {
	details: string
}

Product {
	name: string,
	image: string,
	price: float,
	amount: integer,
	category: Category
}

Seller {
	name: string,
	currentAddress: Address,
	fixedAddress?: Address,
	feedbackRate: integer,
	contact: Contact,
	image: string,
	backgroundImage: string,
	produts: Product[]
}

Buyer {
	name: string,
	username: string,
	password: string,
	contact: Contact
}