type User = {
  id: number;
  name: string;
  email: string;
  type: 'user';
};

type Admin = {
  id: number;
  name: string;
  role: string;
  type: 'admin';
};

type Person = User | Admin;

type Criteria<T> = Omit<Partial<T>, 'type'>;

function filterPersons<T extends 'user' | 'admin'>(
  persons: Person[],
  personType: T,
  criteria: Criteria<T extends 'user' ? User : Admin>
): (T extends 'user' ? User[] : Admin[]) {
  return persons.filter(person => {
    if (person.type !== personType) return false;
    return Object.entries(criteria).every(([key, value]) =>
      (person as any)[key] === value
    );
  }) as any;
}

// Example Usage
const persons: Person[] = [
  { id: 1, name: 'Alice', email: 'alice@example.com', type: 'user' },
  { id: 2, name: 'Bob', role: 'Manager', type: 'admin' },
  { id: 3, name: 'Charlie', email: 'charlie@example.com', type: 'user' },
];

const users = filterPersons(persons, 'user', { name: 'Alice' }); // User[]
const admins = filterPersons(persons, 'admin', { role: 'Manager' }); // Admin[]

console.log(users, admins)
